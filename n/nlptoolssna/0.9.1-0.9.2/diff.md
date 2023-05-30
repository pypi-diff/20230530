# Comparing `tmp/nlptoolssna-0.9.1.tar.gz` & `tmp/nlptoolssna-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlptoolssna-0.9.1.tar", last modified: Wed May 17 17:35:55 2023, max compression
+gzip compressed data, was "nlptoolssna-0.9.2.tar", last modified: Tue May 30 18:28:10 2023, max compression
```

## Comparing `nlptoolssna-0.9.1.tar` & `nlptoolssna-0.9.2.tar`

### file list

```diff
@@ -1,99 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.948094 nlptoolssna-0.9.1/
--rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/HISTORY.rst
--rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1924 2023-05-17 17:35:55.948094 nlptoolssna-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.845288 nlptoolssna-0.9.1/docs/
--rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.9.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.762286 nlptoolssna-0.9.1/docs/build/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.763689 nlptoolssna-0.9.1/docs/build/html/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.846633 nlptoolssna-0.9.1/docs/build/html/_images/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.1/docs/build/html/_images/download.png
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.854958 nlptoolssna-0.9.1/docs/build/html/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.1/docs/build/html/_static/download.png
--rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.9.1/docs/build/html/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.1/docs/build/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.1/docs/build/html/_static/plus.png
--rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.9.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.863547 nlptoolssna-0.9.1/docs/source/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.863547 nlptoolssna-0.9.1/docs/source/_static/
--rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.1/docs/source/_static/download.png
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.871704 nlptoolssna-0.9.1/docs/source/api/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.871704 nlptoolssna-0.9.1/docs/source/api/DataDownload/
--rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.9.1/docs/source/api/DataDownload/downloader.rst
--rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.9.1/docs/source/api/DataDownload.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.871704 nlptoolssna-0.9.1/docs/source/api/morphology/
--rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.9.1/docs/source/api/morphology/morph_analyzer.rst
--rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.9.1/docs/source/api/morphology.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.877229 nlptoolssna-0.9.1/docs/source/api/utils/
--rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.9.1/docs/source/api/utils/implication.rst
--rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.9.1/docs/source/api/utils/jaccard.rst
--rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.9.1/docs/source/api/utils/parser.rst
--rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.9.1/docs/source/api/utils/text_transliteration.rst
--rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.9.1/docs/source/api/utils.rst
--rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.9.1/docs/source/api.rst
--rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.9.1/docs/source/authors.rst
--rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.9.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.9.1/docs/source/index.rst
--rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/docs/source/installation.rst
--rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.9.1/docs/source/readme.rst
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.885888 nlptoolssna-0.9.1/nlptools/
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.885888 nlptoolssna-0.9.1/nlptools/DataDownload/
--rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.9.1/nlptools/DataDownload/__init__.py
--rw-rw-rw-   0        0        0     9187 2023-05-17 17:03:21.000000 nlptoolssna-0.9.1/nlptools/DataDownload/downloader.py
--rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.9.1/nlptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.885888 nlptoolssna-0.9.1/nlptools/arabiner/
--rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.9.1/nlptools/arabiner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.894464 nlptoolssna-0.9.1/nlptools/arabiner/bin/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.1/nlptools/arabiner/bin/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-05-17 16:50:20.000000 nlptoolssna-0.9.1/nlptools/arabiner/bin/eval.py
--rw-rw-rw-   0        0        0     1288 2023-05-17 17:35:16.000000 nlptoolssna-0.9.1/nlptools/arabiner/bin/infer.py
--rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.9.1/nlptools/arabiner/bin/process.py
--rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.9.1/nlptools/arabiner/bin/train.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.902571 nlptoolssna-0.9.1/nlptools/arabiner/data/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.1/nlptools/arabiner/data/__init__.py
--rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.9.1/nlptools/arabiner/data/datasets.py
--rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.9.1/nlptools/arabiner/data/transforms.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.911528 nlptoolssna-0.9.1/nlptools/arabiner/nn/
--rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.9.1/nlptools/arabiner/nn/BaseModel.py
--rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.9.1/nlptools/arabiner/nn/BertNestedTagger.py
--rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.9.1/nlptools/arabiner/nn/BertSeqTagger.py
--rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.9.1/nlptools/arabiner/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.917576 nlptoolssna-0.9.1/nlptools/arabiner/utils/
--rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.1/nlptools/arabiner/utils/__init__.py
--rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.9.1/nlptools/arabiner/utils/data.py
--rw-rw-rw-   0        0        0     3720 2023-05-17 17:35:38.000000 nlptoolssna-0.9.1/nlptools/arabiner/utils/helpers.py
--rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.9.1/nlptools/arabiner/utils/metrics.py
--rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/nlptools/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.917576 nlptoolssna-0.9.1/nlptools/data/
--rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.9.1/nlptools/data/my_data.pickle
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.927023 nlptoolssna-0.9.1/nlptools/morphology/
--rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.9.1/nlptools/morphology/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.9.1/nlptools/morphology/charsets.py
--rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.9.1/nlptools/morphology/morph_analyzer.py
--rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.9.1/nlptools/morphology/settings.py
--rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.9.1/nlptools/morphology/tokenizers_words.py
--rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/nlptools/nlptools.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.937250 nlptoolssna-0.9.1/nlptools/utils/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.9.1/nlptools/utils/__init__.py
--rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.9.1/nlptools/utils/implication.py
--rw-rw-rw-   0        0        0    10287 2023-05-11 20:50:47.000000 nlptoolssna-0.9.1/nlptools/utils/jaccard.py
--rw-rw-rw-   0        0        0     7600 2023-05-15 14:27:42.000000 nlptoolssna-0.9.1/nlptools/utils/parser.py
--rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.9.1/nlptools/utils/text_transliteration.py
--rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.9.1/nlptools/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.948094 nlptoolssna-0.9.1/nlptoolssna.egg-info/
--rw-rw-rw-   0        0        0     1924 2023-05-17 17:35:55.000000 nlptoolssna-0.9.1/nlptoolssna.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2164 2023-05-17 17:35:55.000000 nlptoolssna-0.9.1/nlptoolssna.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 17:35:55.000000 nlptoolssna-0.9.1/nlptoolssna.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-17 17:35:55.000000 nlptoolssna-0.9.1/nlptoolssna.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.9.1/nlptoolssna.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      144 2023-05-17 17:35:55.000000 nlptoolssna-0.9.1/nlptoolssna.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-17 17:35:55.000000 nlptoolssna-0.9.1/nlptoolssna.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-17 17:35:55.948094 nlptoolssna-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0     2095 2023-05-17 07:09:09.000000 nlptoolssna-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 17:35:55.948094 nlptoolssna-0.9.1/tests/
--rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/tests/__init__.py
--rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.9.1/tests/test_nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.965044 nlptoolssna-0.9.2/
+-rw-rw-rw-   0        0        0      172 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3667 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       97 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1091 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1924 2023-05-30 18:28:10.965044 nlptoolssna-0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.831739 nlptoolssna-0.9.2/docs/
+-rw-rw-rw-   0        0        0      676 2023-04-26 19:48:07.000000 nlptoolssna-0.9.2/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.789202 nlptoolssna-0.9.2/docs/build/
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.791206 nlptoolssna-0.9.2/docs/build/html/
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.833741 nlptoolssna-0.9.2/docs/build/html/_images/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.2/docs/build/html/_images/download.png
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.842015 nlptoolssna-0.9.2/docs/build/html/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.2/docs/build/html/_static/download.png
+-rw-rw-rw-   0        0        0      286 2023-04-11 21:34:54.000000 nlptoolssna-0.9.2/docs/build/html/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.2/docs/build/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-04-11 21:34:54.000000 nlptoolssna-0.9.2/docs/build/html/_static/plus.png
+-rwxrwxrwx   0        0        0      791 2023-03-28 19:29:13.000000 nlptoolssna-0.9.2/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.852905 nlptoolssna-0.9.2/docs/source/
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.855723 nlptoolssna-0.9.2/docs/source/_static/
+-rw-rw-rw-   0        0        0     9568 2023-04-26 20:26:03.000000 nlptoolssna-0.9.2/docs/source/_static/download.png
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.863067 nlptoolssna-0.9.2/docs/source/api/
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.865123 nlptoolssna-0.9.2/docs/source/api/DataDownload/
+-rw-rw-rw-   0        0        0      138 2023-05-01 11:11:44.000000 nlptoolssna-0.9.2/docs/source/api/DataDownload/downloader.rst
+-rw-rw-rw-   0        0        0      234 2023-05-01 11:08:11.000000 nlptoolssna-0.9.2/docs/source/api/DataDownload.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.866069 nlptoolssna-0.9.2/docs/source/api/morphology/
+-rw-rw-rw-   0        0        0      148 2023-05-02 18:17:06.000000 nlptoolssna-0.9.2/docs/source/api/morphology/morph_analyzer.rst
+-rw-rw-rw-   0        0        0      230 2023-05-02 18:16:20.000000 nlptoolssna-0.9.2/docs/source/api/morphology.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.874245 nlptoolssna-0.9.2/docs/source/api/utils/
+-rw-rw-rw-   0        0        0      114 2023-05-04 19:55:13.000000 nlptoolssna-0.9.2/docs/source/api/utils/implication.rst
+-rw-rw-rw-   0        0        0      102 2023-05-06 11:51:47.000000 nlptoolssna-0.9.2/docs/source/api/utils/jaccard.rst
+-rw-rw-rw-   0        0        0       99 2023-05-04 19:26:52.000000 nlptoolssna-0.9.2/docs/source/api/utils/parser.rst
+-rw-rw-rw-   0        0        0      141 2023-05-08 19:10:33.000000 nlptoolssna-0.9.2/docs/source/api/utils/text_transliteration.rst
+-rw-rw-rw-   0        0        0      271 2023-05-08 19:09:40.000000 nlptoolssna-0.9.2/docs/source/api/utils.rst
+-rw-rw-rw-   0        0        0      182 2023-05-06 11:52:28.000000 nlptoolssna-0.9.2/docs/source/api.rst
+-rw-rw-rw-   0        0        0       32 2023-04-26 19:28:12.000000 nlptoolssna-0.9.2/docs/source/authors.rst
+-rw-rw-rw-   0        0        0     6180 2023-04-27 12:10:35.000000 nlptoolssna-0.9.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0      314 2023-05-06 11:52:23.000000 nlptoolssna-0.9.2/docs/source/index.rst
+-rw-rw-rw-   0        0        0     1177 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       31 2023-04-26 19:27:50.000000 nlptoolssna-0.9.2/docs/source/readme.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.880272 nlptoolssna-0.9.2/nlptools/
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.883254 nlptoolssna-0.9.2/nlptools/DataDownload/
+-rw-rw-rw-   0        0        0        0 2023-04-16 17:23:41.000000 nlptoolssna-0.9.2/nlptools/DataDownload/__init__.py
+-rw-rw-rw-   0        0        0     9187 2023-05-17 17:03:21.000000 nlptoolssna-0.9.2/nlptools/DataDownload/downloader.py
+-rw-rw-rw-   0        0        0      132 2023-05-06 12:05:24.000000 nlptoolssna-0.9.2/nlptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.885341 nlptoolssna-0.9.2/nlptools/arabiner/
+-rw-rw-rw-   0        0        0        0 2023-02-26 06:10:53.000000 nlptoolssna-0.9.2/nlptools/arabiner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.894867 nlptoolssna-0.9.2/nlptools/arabiner/bin/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-05-29 19:50:55.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/eval.py
+-rw-rw-rw-   0        0        0     2472 2023-05-30 17:36:00.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/infer.py
+-rw-rw-rw-   0        0        0     4698 2023-05-17 16:50:12.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/process.py
+-rw-rw-rw-   0        0        0     6390 2023-05-17 16:47:20.000000 nlptoolssna-0.9.2/nlptools/arabiner/bin/train.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.899868 nlptoolssna-0.9.2/nlptools/arabiner/data/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/data/__init__.py
+-rw-rw-rw-   0        0        0     5068 2023-05-17 16:50:09.000000 nlptoolssna-0.9.2/nlptools/arabiner/data/datasets.py
+-rw-rw-rw-   0        0        0     4878 2023-05-17 16:52:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/data/transforms.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.906524 nlptoolssna-0.9.2/nlptools/arabiner/nn/
+-rw-rw-rw-   0        0        0      608 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/BaseModel.py
+-rw-rw-rw-   0        0        0     1223 2023-05-17 16:45:19.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/BertNestedTagger.py
+-rw-rw-rw-   0        0        0      504 2023-05-17 16:44:20.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/BertSeqTagger.py
+-rw-rw-rw-   0        0        0      155 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.913750 nlptoolssna-0.9.2/nlptools/arabiner/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-17 16:42:37.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/__init__.py
+-rw-rw-rw-   0        0        0     4162 2023-05-17 16:50:05.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/data.py
+-rw-rw-rw-   0        0        0     3720 2023-05-17 17:35:38.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/helpers.py
+-rw-rw-rw-   0        0        0     2734 2023-05-17 16:48:31.000000 nlptoolssna-0.9.2/nlptools/arabiner/utils/metrics.py
+-rw-rw-rw-   0        0        0      458 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/nlptools/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.915749 nlptoolssna-0.9.2/nlptools/data/
+-rw-rw-rw-   0        0        0    86011 2023-04-06 09:01:12.000000 nlptoolssna-0.9.2/nlptools/data/my_data.pickle
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.925396 nlptoolssna-0.9.2/nlptools/morphology/
+-rw-rw-rw-   0        0        0      377 2023-05-02 18:19:19.000000 nlptoolssna-0.9.2/nlptools/morphology/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-04-27 18:35:11.000000 nlptoolssna-0.9.2/nlptools/morphology/charsets.py
+-rw-rw-rw-   0        0        0     6363 2023-05-16 09:08:44.000000 nlptoolssna-0.9.2/nlptools/morphology/morph_analyzer.py
+-rw-rw-rw-   0        0        0       47 2023-04-01 20:02:46.000000 nlptoolssna-0.9.2/nlptools/morphology/settings.py
+-rw-rw-rw-   0        0        0      602 2023-05-11 20:52:05.000000 nlptoolssna-0.9.2/nlptools/morphology/tokenizers_words.py
+-rw-rw-rw-   0        0        0       20 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/nlptools/nlptools.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.930740 nlptoolssna-0.9.2/nlptools/salma/
+-rw-rw-rw-   0        0        0        0 2023-04-06 11:46:10.000000 nlptoolssna-0.9.2/nlptools/salma/__init__.py
+-rw-rw-rw-   0        0        0    17930 2023-05-20 20:02:01.000000 nlptoolssna-0.9.2/nlptools/salma/views.py
+-rw-rw-rw-   0        0        0     7719 2023-05-20 20:02:29.000000 nlptoolssna-0.9.2/nlptools/salma/wsd.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.947367 nlptoolssna-0.9.2/nlptools/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:33:56.000000 nlptoolssna-0.9.2/nlptools/utils/__init__.py
+-rw-rw-rw-   0        0        0     4706 2023-05-29 19:21:39.000000 nlptoolssna-0.9.2/nlptools/utils/corpus.py
+-rw-rw-rw-   0        0        0    27932 2023-05-16 09:08:16.000000 nlptoolssna-0.9.2/nlptools/utils/implication.py
+-rw-rw-rw-   0        0        0    10160 2023-05-22 14:31:38.000000 nlptoolssna-0.9.2/nlptools/utils/jaccard.py
+-rw-rw-rw-   0        0        0     6144 2023-05-22 14:15:55.000000 nlptoolssna-0.9.2/nlptools/utils/parser.py
+-rw-rw-rw-   0        0        0     8839 2023-05-13 15:09:46.000000 nlptoolssna-0.9.2/nlptools/utils/text_transliteration.py
+-rw-rw-rw-   0        0        0     1201 2023-05-29 19:17:26.000000 nlptoolssna-0.9.2/nlptools/utils/tokenizer.py
+-rw-rw-rw-   0        0        0       32 2023-05-06 10:35:53.000000 nlptoolssna-0.9.2/nlptools/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.959528 nlptoolssna-0.9.2/nlptoolssna.egg-info/
+-rw-rw-rw-   0        0        0     1924 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-06 10:36:33.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      144 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 18:28:10.000000 nlptoolssna-0.9.2/nlptoolssna.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-30 18:28:10.966854 nlptoolssna-0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0     2095 2023-05-17 07:09:09.000000 nlptoolssna-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:28:10.963911 nlptoolssna-0.9.2/tests/
+-rw-rw-rw-   0        0        0       39 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      413 2023-04-15 18:20:16.000000 nlptoolssna-0.9.2/tests/test_nlptools.py
```

### Comparing `nlptoolssna-0.9.1/CONTRIBUTING.rst` & `nlptoolssna-0.9.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/LICENSE` & `nlptoolssna-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/PKG-INFO` & `nlptoolssna-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.9.1/README.rst` & `nlptoolssna-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/docs/Makefile` & `nlptoolssna-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/docs/build/html/_images/download.png` & `nlptoolssna-0.9.2/docs/build/html/_images/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/docs/build/html/_static/download.png` & `nlptoolssna-0.9.2/docs/build/html/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/docs/make.bat` & `nlptoolssna-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/docs/source/_static/download.png` & `nlptoolssna-0.9.2/docs/source/_static/download.png`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/docs/source/conf.py` & `nlptoolssna-0.9.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/docs/source/installation.rst` & `nlptoolssna-0.9.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/DataDownload/downloader.py` & `nlptoolssna-0.9.2/nlptools/DataDownload/downloader.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/bin/eval.py` & `nlptoolssna-0.9.2/nlptools/arabiner/bin/eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,55 @@
 import os
 import logging
-import argparse
 from collections import namedtuple
 from nlptools.arabiner.utils.helpers import load_checkpoint, make_output_dirs, logging_config
 from nlptools.arabiner.utils.data import get_dataloaders, parse_conll_files
 from nlptools.arabiner.utils.metrics import compute_single_label_metrics, compute_nested_metrics
-
+from nlptools.DataDownload import downloader
 logger = logging.getLogger(__name__)
 
 
-def parse_args():
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-    )
-
-    parser.add_argument(
-        "--output_path",
-        type=str,
-        required=True,
-        help="Path to save results",
-    )
-
-    parser.add_argument(
-        "--model_path",
-        type=str,
-        required=True,
-        help="Model path",
-    )
-
-    parser.add_argument(
-        "--data_paths",
-        nargs="+",
-        type=str,
-        required=True,
-        help="Text or sequence to tag, this is in same format as training data with 'O' tag for all tokens",
-    )
-
-    parser.add_argument(
-        "--batch_size",
-        type=int,
-        default=32,
-        help="Batch size",
-    )
-
-    args = parser.parse_args()
-
-    return args
-
-
-def main(args):
+def evaluate_dataset(output_path,data_paths ,batch_size=32):
+    """
+    Run the model to evaluate text data and save the predictions.
+
+    Args:
+        output_path (str): Path to save the results.
+        model_path (str): Model path.
+        data_paths (list[str]): List of paths to text or sequence files to tag.
+        batch_size (int, optional): Batch size. Default is 32.
+    """
     # Create directory to save predictions
-    make_output_dirs(args.output_path, overwrite=True)
-    logging_config(log_file=os.path.join(args.output_path, "eval.log"))
-
+    make_output_dirs(output_path, overwrite=True)
+    logging_config(log_file=os.path.join(output_path, "eval.log"))
+    filename = 'Wj27012000.tar'
+    path =downloader.get_appdatadir()
+    model_path = os.path.join(path, filename)
     # Load tagger
-    tagger, tag_vocab, train_config = load_checkpoint(args.model_path)
+    tagger, tag_vocab, train_config = load_checkpoint(model_path)
 
     # Convert text to a tagger dataset and index the tokens in args.text
-    datasets, vocab = parse_conll_files(args.data_paths)
+    datasets, vocab = parse_conll_files(data_paths)
 
     vocabs = namedtuple("Vocab", ["tags", "tokens"])
     vocab = vocabs(tokens=vocab.tokens, tags=tag_vocab)
 
     # From the datasets generate the dataloaders
     dataloaders = get_dataloaders(
         datasets, vocab,
         train_config.data_config,
-        batch_size=args.batch_size,
+        batch_size=batch_size,
         shuffle=[False] * len(datasets)
     )
 
     # Evaluate the model on each dataloader
-    for dataloader, input_file in zip(dataloaders, args.data_paths):
+    for dataloader, input_file in zip(dataloaders,data_paths):
         filename = os.path.basename(input_file)
-        predictions_file = os.path.join(args.output_path, f"predictions_{filename}")
+        predictions_file = os.path.join(output_path, f"predictions_{filename}")
         _, segments, _, _ = tagger.eval(dataloader)
         tagger.segments_to_file(segments, predictions_file)
 
         if "Nested" in train_config.trainer_config["fn"]:
             compute_nested_metrics(segments, vocab.tags[1:])
         else:
             compute_single_label_metrics(segments)
 
-
-if __name__ == "__main__":
-    main(parse_args())
```

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/bin/process.py` & `nlptoolssna-0.9.2/nlptools/arabiner/bin/process.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/bin/train.py` & `nlptoolssna-0.9.2/nlptools/arabiner/bin/train.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/data/datasets.py` & `nlptoolssna-0.9.2/nlptools/arabiner/data/datasets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/data/transforms.py` & `nlptoolssna-0.9.2/nlptools/arabiner/data/transforms.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/nn/BaseModel.py` & `nlptoolssna-0.9.2/nlptools/arabiner/nn/BaseModel.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/nn/BertNestedTagger.py` & `nlptoolssna-0.9.2/nlptools/arabiner/nn/BertNestedTagger.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/utils/data.py` & `nlptoolssna-0.9.2/nlptools/arabiner/utils/data.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/utils/helpers.py` & `nlptoolssna-0.9.2/nlptools/arabiner/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/arabiner/utils/metrics.py` & `nlptoolssna-0.9.2/nlptools/arabiner/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/data/my_data.pickle` & `nlptoolssna-0.9.2/nlptools/data/my_data.pickle`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/morphology/charsets.py` & `nlptoolssna-0.9.2/nlptools/morphology/charsets.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/morphology/morph_analyzer.py` & `nlptoolssna-0.9.2/nlptools/morphology/morph_analyzer.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/morphology/tokenizers_words.py` & `nlptoolssna-0.9.2/nlptools/morphology/tokenizers_words.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/utils/implication.py` & `nlptoolssna-0.9.2/nlptools/utils/implication.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptools/utils/jaccard.py` & `nlptoolssna-0.9.2/nlptools/utils/jaccard.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,47 +5,46 @@
 @author: Tymaa
 """
 
 from nlptools.utils.parser import arStrip
 from nlptools.utils.implication import Implication
 
 
-def normalize_word(word: str, ignore_all_diacritics_but_not_shadda: bool, ignore_shadda_diacritic: bool) -> str:
+def normalize_word(word: str, ignore_all_diacritics_but_not_shadda: bool=True, ignore_shadda_diacritic: bool=True) -> str:
     """
-    Normalize a given Arabic word by removing diacritics and/or shadda diacritic based on the provided flags.
+    Normalize a given Arabic word by removing diacritics and/or shadda diacritic.
 
     Args:
-        word (:obj:`str`): A string representing an Arabic word to be normalized.
-        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A boolean flag indicating whether to remove all diacritics except shadda.
-        ignore_shadda_diacritic (:obj:`bool`): A boolean flag indicating whether to remove shadda diacritic.
+        word (:obj:`str`): The input text.
+        ignore_all_diacritics_but_not_shadda (:obj:`bool`): A boolean flag indicating whether to remove all diacritics except shadda (default is True). 
+        ignore_shadda_diacritic (:obj:`bool`): A boolean flag indicating whether to remove shadda diacritic (default is True).
 
     Returns:
-        A string representing the normalized Arabic word.
+          :obj:`str` Normalized Arabic word.
     """
     if ignore_all_diacritics_but_not_shadda:
-        # Remove all diacritics except shadda
         word = arStrip(word, True, True, False, False, False, False)
         
     if ignore_shadda_diacritic:
-        # Remove shadda diacritic
         word = arStrip(word, False, False, True, False, False, False)
     
     return word
 
     
 def get_preferred_word(word1, word2):
     """
     Returns the preferred word among two given words based on their implication.
 
     Args:
-        word1 (:obj:`str`): The first word to be compared.
-        word2 (:obj:`str`): The second word to be compared.
+        word1 (:obj:`str`): The first word.
+        word2 (:obj:`str`): The second word.
 
     Returns:
-        str: The preferred word among the two given words.
+        :obj:`str`: The preferred word among the two given words.
+    
     """
     implication = Implication(word1, word2)
     
     direction = implication.get_direction()
     
     if direction in (0, 2):
         return word1
@@ -57,38 +56,38 @@
         if not word1.endswith("َ") and not word1.endswith("ُ"):
             return word2
         return word1
      
     
 def get_non_preferred_word(word1, word2):
     """
-    Find the non-preferred word between the two input words.
+    Returns the non-preferred word between the two input words.
 
     Args:
         word1 (:obj:`str`): The first word.
         word2 (:obj:`str`): The second word.
 
     Returns:
-        :obj:`str`: The non-preferred word. If there is no non-preferred word, returns '#'.
+        :obj:`str`: The non-preferred word. If there is no non-preferred word, The '#' is returned.
 
     """
-    # Find non-preferred word if the distance between the two words input is less than 15.
+
     implication = Implication(word1, word2)
     if implication.get_distance() < 15:
         direction = implication.get_direction()
         if direction == 0 or direction == 1:
             return word1
         elif direction == 2:
             return word2
         elif direction == 3:
             if not word1.endswith("َ") and not word1.endswith("ُ"):
                 return word1
             return word2
     return "#"
-
+@TBD
 def get_intersection(list1, list2, ignore_all_diacritics_but_not_shadda=False, ignore_shadda_diacritic=False):
     """
     Get the intersection of two lists after normalization and ignoring diacritics based on input flags.
 
     Args:
         list1 (:obj:`list`): The first list.
         list2 (:obj:`list`): The second list.
@@ -217,14 +216,15 @@
         The Jaccard similarity, union, or intersection of the two sets of strings, 
         depending on the value of the `selection` argument.
     
     Note:
         - If `selection` is *jaccardAll*, a list of the intersection, union, and Jaccard similarity 
         of the two sets of strings will be returned.
         - If an error occurs, the method will return the string "An error has occurred".
+          Online tool: https://sina.birzeit.edu/resources/jaccardFunction.html
     """
     try:
         list1 = str1.split(delimiter)
         list2 = str2.split(delimiter)
 
         if selection == "intersection":
             intersection = get_intersection(list1, list2, ignoreAllDiacriticsButNotShadda, ignoreShaddaDiacritic)
```

### Comparing `nlptoolssna-0.9.1/nlptools/utils/text_transliteration.py` & `nlptoolssna-0.9.2/nlptools/utils/text_transliteration.py`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/nlptoolssna.egg-info/PKG-INFO` & `nlptoolssna-0.9.2/nlptoolssna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlptoolssna
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/eng-aomar/nlptools
 Author: Alaa' Omar
 Author-email: alaa.omer2009@gmail.com
 License: MIT license
 Keywords: nlptools
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `nlptoolssna-0.9.1/nlptoolssna.egg-info/SOURCES.txt` & `nlptoolssna-0.9.2/nlptoolssna.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -53,19 +53,24 @@
 nlptools/arabiner/utils/metrics.py
 nlptools/data/my_data.pickle
 nlptools/morphology/__init__.py
 nlptools/morphology/charsets.py
 nlptools/morphology/morph_analyzer.py
 nlptools/morphology/settings.py
 nlptools/morphology/tokenizers_words.py
+nlptools/salma/__init__.py
+nlptools/salma/views.py
+nlptools/salma/wsd.py
 nlptools/utils/__init__.py
+nlptools/utils/corpus.py
 nlptools/utils/implication.py
 nlptools/utils/jaccard.py
 nlptools/utils/parser.py
 nlptools/utils/text_transliteration.py
+nlptools/utils/tokenizer.py
 nlptools/utils/utils.py
 nlptoolssna.egg-info/PKG-INFO
 nlptoolssna.egg-info/SOURCES.txt
 nlptoolssna.egg-info/dependency_links.txt
 nlptoolssna.egg-info/entry_points.txt
 nlptoolssna.egg-info/not-zip-safe
 nlptoolssna.egg-info/requires.txt
```

### Comparing `nlptoolssna-0.9.1/setup.cfg` & `nlptoolssna-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nlptoolssna-0.9.1/setup.py` & `nlptoolssna-0.9.2/setup.py`

 * *Files identical despite different names*

